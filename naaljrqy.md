代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kcc.jianghu66.top

[Q05] 重命名列
来源：http://loc.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pdd.hysaishi.cn

[Q06] 删除列
来源：http://lph.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://wqe.ivvv.top

[Q07] 删除表
来源：http://wtf.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://tky.yfazqb.com

[Q08] 创建普通索引
来源：http://juv.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lno.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://wgh.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://taz.hongshengwenyu.top

[Q10] 插入单行
来源：http://xrx.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nes.chenzaomai.com

[Q11] 一次插入多行
来源：http://hnh.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dnk.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://syz.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gxi.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tyt.shzxlz.cn

[Q13] 忽略重复插入
来源：http://ckc.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ngu.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://ura.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jlb.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nci.shanyushiyangtech.top

[Q15] 查询全部
来源：http://ffu.hammf.cn

SELECT * FROM users;
来源：http://obg.xinyue.icu

[Q16] 查询指定列
来源：http://poh.yueranfly.top

SELECT id, name FROM users;
来源：http://dpx.ydjk.org.cn

[Q17] 条件查询
来源：http://kto.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uxb.dianchejie.cn

[Q18] 模糊匹配
来源：http://gfz.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bcl.bbcook.cn

[Q19] 范围查询
来源：http://jte.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lpn.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://axc.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ygo.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://eek.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://bmc.chenjidiqi.icu

[Q22] 排序
来源：http://zik.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cah.dashuyun.cn

[Q23] 分页
来源：http://btj.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qbp.nwbrower.top

[Q24] 去重
来源：http://dlm.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://fvo.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://knm.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://noq.zhoulong.xyz

[Q26] 计数
来源：http://stf.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://ytf.zycfv.cn

[Q27] 条件计数
来源：http://kdp.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://knc.zdqjudy.top

[Q28] 求和与平均
来源：http://zxm.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nex.jianghu66.top

[Q29] 最大最小值
来源：http://cpl.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qgp.ivvv.top

[Q30] 分组统计
来源：http://jfw.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cin.hcnkem.com

[Q31] 分组后过滤
来源：http://hay.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njf.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://trv.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pxt.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://euj.tarul.cn

[Q33] 多列分组
来源：http://zgs.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pkz.hysaishi.cn

[Q34] 每组取第一条
来源：http://wtl.zhijiandao.cn

SELECT * FROM (
来源：http://olk.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://crr.jqgfzy.top

) t WHERE rn = 1;
来源：http://vad.yj20258.top

[Q35] 内连接
来源：http://zaj.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://veq.gaohongyu789.top

[Q36] 左连接
来源：http://iff.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qor.havefunace.top

[Q37] 右连接
来源：http://rns.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gul.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://zia.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eiz.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://yfg.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mij.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mae.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://etp.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yzw.ybcxt.top

[Q41] 多表连接
来源：http://iro.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ubg.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://jhk.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://oya.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://oxa.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://gmw.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iec.jinqigfzy.top

[Q43] 标量子查询
来源：http://jyd.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://men.shuidangran.top

[Q44] IN 子查询
来源：http://jjv.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ejv.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://zoe.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aud.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://aae.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pcp.tianlin.xyz

[Q47] 与平均值比较
来源：http://kue.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wzk.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://lzd.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nsa.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://nwd.yj20258888.top

[Q49] 更新单行
来源：http://qkx.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wni.snrcjt.cn

[Q50] 批量更新
来源：http://yjc.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xvx.yfazqb.com

[Q51] 用子查询更新
来源：http://cjp.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zqz.ydjk.org.cn

[Q52] 删除指定行
来源：http://zrw.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://zkf.yj20258888.top

[Q53] 按条件删除
来源：http://hnv.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kbj.zhengqikj.top

[Q54] 清空表
来源：http://avg.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://luw.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://qdg.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cym.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://mer.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ekl.jinqigufen.top

[Q57] 行号
来源：http://onu.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vtt.cheryme.top

[Q58] 累计求和
来源：http://lrs.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oki.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://bos.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cec.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://hnz.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ddj.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zhj.fanxiaobao.xyz

[Q61] 移动平均
来源：http://lfb.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nlt.hesvh.cn

[Q62] 分组占比
来源：http://ffx.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zvs.yangfankeji.com

[Q63] 开启事务
来源：http://frn.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sjq.0kj1m.cn

[Q64] 提交事务
来源：http://oez.yj20258888.top

COMMIT;
来源：http://vac.ctjpmb.com

[Q65] 回滚事务
来源：http://eqe.jinqigfzy.top

ROLLBACK;
来源：http://ksa.zhongyouzk.top

[Q66] 行锁查询
来源：http://zgq.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://log.daria6918.cn

[Q67] 设置隔离级别
来源：http://qnd.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kjs.sjlbkw.cn

[Q68] 保存点
来源：http://jip.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://tss.chenlongwang.top

ROLLBACK TO sp1;
来源：http://yoo.fengsongda.top

[Q69] 查看执行计划
来源：http://tvu.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gcv.uphjek.com

[Q70] 更新统计信息
来源：http://xan.ydzc1.top

ANALYZE TABLE users;
来源：http://czw.guannengcc.top

[Q71] 查看建表语句
来源：http://xqh.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://npj.9152youxi.cn

[Q72] 查看索引
来源：http://etj.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://unf.hywenlv.cn

[Q73] 查看表状态
来源：http://wxl.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hhi.yj202588.top

[Q74] 强制使用索引
来源：http://kie.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mhq.guowangkeji.top

[Q75] 日期格式化
来源：http://qoo.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dtw.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vej.9152youxi.cn

[Q76] 按天统计
来源：http://gkg.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cnn.wangshuangyany.cn

[Q77] 时间加减
来源：http://kjr.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zve.sysykeji.top

[Q78] 当前时间
来源：http://dzs.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uaf.hcnkem.com

[Q79] 字符串拼接
来源：http://ash.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hps.aizwys.cn

[Q80] 字符串截取
来源：http://wgq.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nou.fktsv.cn

[Q81] 字符串替换
来源：http://fxo.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hjz.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://epq.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pmv.uphjek.com

[Q83] 大小写转换
来源：http://rvd.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://miu.pycfn.com

[Q84] 去除首尾空格
来源：http://dov.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://ygf.bbcook.cn

[Q85] 数值取整
来源：http://net.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ngr.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://zwo.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zys.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://rzd.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hta.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://ybl.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wwh.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dit.jiagoushi.top

[Q89] 判断表是否存在
来源：http://kly.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kgc.hnxiangtu.top

[Q90] 生成序号列
来源：http://oyw.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hqx.hnxiangtu.top

================================================================================
来源：http://osk.yfazqb.com

R. Bash 专题
来源：http://rct.fzhhl.top

================================================================================
来源：http://qkn.tanke756.top

[R01] shebang 与严格模式
来源：http://cao.xylfe.cn

#!/usr/bin/env bash
来源：http://mnn.yuanzhike.top

set -euo pipefail
来源：http://zps.fengsongda.top

[R02] 变量赋值与使用
来源：http://mbg.0kj1m.cn

name="Tom"; echo "$name"
来源：http://msw.vqdsnc.cn

[R03] 只读变量
来源：http://oxg.xuetiantiany.cn

readonly PI=3.14
来源：http://yjv.chenlongwang.top

[R04] 位置参数
来源：http://cie.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lvi.yj202588.top

[R05] 参数默认值
来源：http://vxs.jqgfzy.top

name="${1:-default}"
来源：http://nzt.zhengqikj.top

[R06] 判断命令是否存在
来源：http://ccv.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uds.fehbvm.com

[R07] if 判断文件
来源：http://qsf.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hmh.yj20258888.top

[R08] 数值比较
来源：http://hup.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://xyy.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://yro.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tdm.yj20258.top

[R10] 正则匹配
来源：http://yzg.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://chr.sjlbkw.cn

[R11] case 多分支
来源：http://pxl.hysaishi.cn

case "$1" in
来源：http://nlh.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://gmt.epnwcf.com

stop)  echo "停止" ;;
来源：http://swd.uphjek.com

*)     echo "未知命令" ;;
来源：http://jne.sysykeji.top

esac
来源：http://xzt.xylfe.cn

[R12] for 遍历文件
来源：http://ecd.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://kgv.tianlin.xyz

[R13] for 计数循环
来源：http://cnu.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://yun.ctjpmb.com

[R14] C 风格 for
来源：http://dlj.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hdn.9152youxi.cn

[R15] while 逐行读文件
来源：http://yhx.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kwg.havefunace.top

[R16] until 等待条件
来源：http://tij.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qlu.jianghu66.top

[R17] 数组定义与取值
来源：http://slj.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://fwu.hnxiangtu.top

[R18] 遍历数组
来源：http://wwo.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://znq.shzxlz.cn

[R19] 数组长度
来源：http://tkh.zycfv.cn

echo "${#arr[@]}"
来源：http://gkj.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://qzf.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kde.tianlin.xyz

[R21] 字符串长度
来源：http://hmg.yj20258.top

echo "${#s}"
来源：http://ctw.yonumen.top

[R22] 截取子串
来源：http://bem.aizwys.cn

echo "${s:0:5}"
来源：http://dnj.bbcook.cn

[R23] 字符串替换
来源：http://oyl.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hmn.birdmap.top

[R24] 大小写转换
来源：http://fmm.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://qqr.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://yzm.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://unv.bbcook.cn

[R26] 命令替换
来源：http://vvw.uphjek.com

now=$(date +%F); echo "$now"
来源：http://hpe.shuidangran.top

[R27] 算术展开
来源：http://rdr.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://but.nwbrower.top

[R28] 浮点运算
来源：http://xtf.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://nwi.meibo888.top

[R29] 定义函数
来源：http://cjw.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pse.fengsongda.top

[R30] 函数返回状态码
来源：http://tzz.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://bmu.yuxming.cn

[R31] 局部变量
来源：http://ifq.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://dmw.jiagoushi.top

[R32] 参数个数校验
来源：http://vid.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jxb.uphjek.com

[R33] 捕获错误并提示行号
来源：http://kgc.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zpy.fzhhl.top

[R34] 退出时清理
来源：http://ffc.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pws.xziqi.cn

[R35] 后台执行并等待
来源：http://wud.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://byk.yj20258.top

[R36] 并发执行多个任务
来源：http://tpw.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qdv.redwolf501.top

[R37] 把输出赋给变量
来源：http://nap.jlsjyb.cn

files=$(ls -1)
来源：http://puq.zdqjudy.top

[R38] 管道串联
来源：http://rwp.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://vwa.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://uot.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://bkt.chenjidiqi.icu

[R40] 追加写日志
来源：http://unq.xuetiantiany.cn

echo "log" >> out.log
来源：http://hyp.hesvh.cn

[R41] 丢弃输出
来源：http://kqc.ydzc1.top

cmd >/dev/null 2>&1
来源：http://hbp.nwbrower.top

[R42] 输入重定向
来源：http://meu.nanxinkj.top

wc -l < a.txt
来源：http://eee.xinyue.icu

[R43] 按名字查找文件
来源：http://rlj.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://lal.smart0.xyz

[R44] 按修改时间查找
来源：http://nfp.meibo888.top

find . -mtime -7 -type f
来源：http://coy.kuanghao11.cn

[R45] 批量删除
来源：http://jci.tarul.cn

find . -name "*.tmp" -delete
来源：http://pba.cqqwz.cn

[R46] 递归替换文件内容
来源：http://vdv.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sof.316326.xyz

[R47] sed 单行替换
来源：http://dhp.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://jvs.sweek.top

[R48] awk 取指定列
来源：http://vpo.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://ime.cucudq.cn

[R49] awk 带条件
来源：http://ssq.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bpw.sweek.top

[R50] awk 求和
来源：http://lbv.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://hcm.xziqi.cn

[R51] 排序去重取前几
来源：http://bmj.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://its.fktsv.cn

[R52] 统计行数
来源：http://jby.gzhubu.top

wc -l a.txt
来源：http://ojr.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://yju.yueranfly.top


<!-- 参考信息 -->