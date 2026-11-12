代发 wailian999

CREATE TABLE users (
来源：http://sbd.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jwy.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://twy.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://xcr.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dpq.cashguo.top

);
来源：http://jat.0kj1m.cn

[Q02] 创建带外键的表
来源：http://mzr.gogol.net.cn

CREATE TABLE orders (
来源：http://wgw.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qad.svipenyu.cn

user_id INT NOT NULL,
来源：http://dcz.yvedp.cn

amount DECIMAL(10, 2),
来源：http://mub.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fie.cdnleiting.top

);
来源：http://jip.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://yah.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mps.vqdsnc.cn

[Q04] 修改列类型
来源：http://qcc.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rlo.wangdashe.top

[Q05] 重命名列
来源：http://zhr.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gtu.nanxinkj.top

[Q06] 删除列
来源：http://fpj.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://igd.ehwqpu.com

[Q07] 删除表
来源：http://xig.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://kyx.sjlbkw.cn

[Q08] 创建普通索引
来源：http://ptg.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://vdy.guowangkeji.top

[Q09] 创建唯一索引
来源：http://pzn.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://icb.dianchejie.cn

[Q10] 插入单行
来源：http://oit.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mom.yanxiufei.cn

[Q11] 一次插入多行
来源：http://zjv.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://adc.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://izs.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://pgw.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cms.yvedp.cn

[Q13] 忽略重复插入
来源：http://ryl.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fca.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://hhy.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lyh.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uej.birdmap.top

[Q15] 查询全部
来源：http://yfy.yanxiufei.cn

SELECT * FROM users;
来源：http://qvw.sjlbkw.cn

[Q16] 查询指定列
来源：http://fto.bbcook.cn

SELECT id, name FROM users;
来源：http://lfh.xuanzx.com

[Q17] 条件查询
来源：http://zgs.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yqu.dianchejie.cn

[Q18] 模糊匹配
来源：http://wzf.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ekc.epnwcf.com

[Q19] 范围查询
来源：http://wbq.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epy.hywenlv.cn

[Q20] IN 列表
来源：http://oxd.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qmb.yfazqb.com

[Q21] 空值判断
来源：http://ydp.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wgt.uphjek.com

[Q22] 排序
来源：http://ejg.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bmb.jiagoushi.top

[Q23] 分页
来源：http://qqv.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rwj.zycfv.cn

[Q24] 去重
来源：http://unb.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://lxp.fktsv.cn

[Q25] 只取前 N 条
来源：http://zyw.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://toc.yanxiufei.cn

[Q26] 计数
来源：http://jqn.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://lxf.52xcode.cn

[Q27] 条件计数
来源：http://oia.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mqi.cheryme.top

[Q28] 求和与平均
来源：http://hua.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hpo.sweek.top

[Q29] 最大最小值
来源：http://xcy.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yck.uphjek.com

[Q30] 分组统计
来源：http://kzn.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xml.ybcxt.top

[Q31] 分组后过滤
来源：http://oga.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yei.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://ame.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zpw.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lhc.shangyingyoupin.top

[Q33] 多列分组
来源：http://eak.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://srf.0kj1m.cn

[Q34] 每组取第一条
来源：http://qja.aizwys.cn

SELECT * FROM (
来源：http://zux.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qrm.cdnleiting.top

) t WHERE rn = 1;
来源：http://oiv.shanyushiyangtech.top

[Q35] 内连接
来源：http://tdq.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mug.haohaochexian.top

[Q36] 左连接
来源：http://mms.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bzg.jinqigfzy.top

[Q37] 右连接
来源：http://xnc.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bcq.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://qpp.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oyt.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://izu.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ers.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://her.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ltk.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lgx.zycfv.cn

[Q41] 多表连接
来源：http://tkm.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nkf.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://glq.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://xbb.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://mvc.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://dhz.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jvb.ehwqpu.com

[Q43] 标量子查询
来源：http://vrr.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kwk.meibo888.top

[Q44] IN 子查询
来源：http://vme.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://piz.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://mjv.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qju.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wez.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://euu.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://qlp.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yis.uphjek.com

[Q48] CTE 公用表表达式
来源：http://ipc.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tda.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://pwz.havefunace.top

[Q49] 更新单行
来源：http://ped.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://brz.mhx1999.top

[Q50] 批量更新
来源：http://qst.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pwl.xuanzx.com

[Q51] 用子查询更新
来源：http://dll.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lxx.daria6918.cn

[Q52] 删除指定行
来源：http://cpe.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://ehr.zhoulong.xyz

[Q53] 按条件删除
来源：http://nkj.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://upw.pengpengdd.cyou

[Q54] 清空表
来源：http://ffx.yj20258.top

TRUNCATE TABLE logs;
来源：http://elf.yongpay.top

[Q55] 排名（并列占位）
来源：http://gsw.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xzx.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://ykn.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mzs.birdmap.top

[Q57] 行号
来源：http://clt.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xpw.tian-w.cn

[Q58] 累计求和
来源：http://wyt.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mdw.gotoacloud.top

[Q59] 分组内累计
来源：http://tel.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tqa.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://dgo.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rrb.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://azn.mhx1999.top

[Q61] 移动平均
来源：http://obe.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://udr.haohaochexian.top

[Q62] 分组占比
来源：http://fmf.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://frg.c1oappe.top

[Q63] 开启事务
来源：http://uol.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://jte.jlsjyb.cn

[Q64] 提交事务
来源：http://bpw.havefunace.top

COMMIT;
来源：http://req.feifeiyinyue.top

[Q65] 回滚事务
来源：http://uaq.cqqwz.cn

ROLLBACK;
来源：http://sgu.tarul.cn

[Q66] 行锁查询
来源：http://pvo.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fxn.jqgfzy.top

[Q67] 设置隔离级别
来源：http://huv.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jcg.nanxinkj.top

[Q68] 保存点
来源：http://ufj.kuanghao11.cn

SAVEPOINT sp1;
来源：http://aht.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://vki.xinyue.icu

[Q69] 查看执行计划
来源：http://tcp.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eqz.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://hmt.yj202588.top

ANALYZE TABLE users;
来源：http://mlo.hesvh.cn

[Q71] 查看建表语句
来源：http://tmi.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yrh.jlsjyb.cn

[Q72] 查看索引
来源：http://yic.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://hve.yangfankeji.com

[Q73] 查看表状态
来源：http://cnc.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gaa.cheryme.top

[Q74] 强制使用索引
来源：http://pzq.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://skd.yvedp.cn

[Q75] 日期格式化
来源：http://fyc.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://esl.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lrx.xuanzx.com

[Q76] 按天统计
来源：http://aiy.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://axz.yj20258.top

[Q77] 时间加减
来源：http://gwh.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kne.aizwys.cn

[Q78] 当前时间
来源：http://ygy.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://npq.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://jid.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ius.shuidangran.top

[Q80] 字符串截取
来源：http://qty.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pey.ydjk.org.cn

[Q81] 字符串替换
来源：http://ibt.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://elh.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://ofx.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gza.yj20258888.top

[Q83] 大小写转换
来源：http://ttm.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://poi.zhengqikj.top

[Q84] 去除首尾空格
来源：http://tbm.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://ybp.vqdsnc.cn

[Q85] 数值取整
来源：http://sio.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mqk.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://deg.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://olt.havefunace.top

[Q87] JSON 字段做条件
来源：http://mub.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zru.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://ubo.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://osa.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://flr.ybcxt.top

[Q89] 判断表是否存在
来源：http://snc.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xlb.nwbrower.top

[Q90] 生成序号列
来源：http://mqo.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://diu.uphjek.com

================================================================================
来源：http://dxf.xinyue.icu

R. Bash 专题
来源：http://fcp.wangshuangyany.cn

================================================================================
来源：http://oxd.mhx1999.top

[R01] shebang 与严格模式
来源：http://vho.cashguo.top

#!/usr/bin/env bash
来源：http://fog.iojbl.cn

set -euo pipefail
来源：http://bfk.ctjpmb.com

[R02] 变量赋值与使用
来源：http://rnm.daxiang520.top

name="Tom"; echo "$name"
来源：http://qmx.iojbl.cn

[R03] 只读变量
来源：http://vbj.yongpay.top

readonly PI=3.14
来源：http://uhb.ppjwa.cn

[R04] 位置参数
来源：http://xzd.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://shc.meibo888.top

[R05] 参数默认值
来源：http://abl.316326.xyz

name="${1:-default}"
来源：http://ugs.c1oappe.top

[R06] 判断命令是否存在
来源：http://dlp.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ses.havefunace.top

[R07] if 判断文件
来源：http://mrx.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tum.iojbl.cn

[R08] 数值比较
来源：http://ktb.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://col.ybcxt.top

[R09] 字符串比较
来源：http://mqv.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qle.kuanghao11.cn

[R10] 正则匹配
来源：http://rna.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vid.0kj1m.cn

[R11] case 多分支
来源：http://mwq.0kj1m.cn

case "$1" in
来源：http://oij.cdnleiting.top

start) echo "启动" ;;
来源：http://zxe.zhixingplan.top

stop)  echo "停止" ;;
来源：http://skw.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://yqx.ivvv.top

esac
来源：http://fgr.xziqi.cn

[R12] for 遍历文件
来源：http://nwx.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://cjz.gotoacloud.top

[R13] for 计数循环
来源：http://haw.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://ira.yueranfly.top

[R14] C 风格 for
来源：http://ldc.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ahq.zdbjq.cn

[R15] while 逐行读文件
来源：http://ohd.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rnf.fzhhl.top

[R16] until 等待条件
来源：http://ndc.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://avx.ppjwa.cn

[R17] 数组定义与取值
来源：http://qvp.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://dtd.jlsjyb.cn

[R18] 遍历数组
来源：http://ttp.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://owf.zhaomingkeji.xyz

[R19] 数组长度
来源：http://uuk.shzxlz.cn

echo "${#arr[@]}"
来源：http://anw.haohaochexian.top

[R20] 关联数组（字典）
来源：http://sof.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://col.nwbrower.top

[R21] 字符串长度
来源：http://vct.yj20258888.top

echo "${#s}"
来源：http://vwa.tanke756.top

[R22] 截取子串
来源：http://jfk.0kj1m.cn

echo "${s:0:5}"
来源：http://dhz.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://xlt.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mfu.havefunace.top

[R24] 大小写转换
来源：http://oqn.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://swi.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://mwb.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cjm.316326.xyz

[R26] 命令替换
来源：http://bzn.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://cdp.haohaochexian.top

[R27] 算术展开
来源：http://iwu.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://jwa.hfpthk.cn

[R28] 浮点运算
来源：http://lfd.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://ivd.chenzaomai.com

[R29] 定义函数
来源：http://ogf.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qfi.ydjk.org.cn

[R30] 函数返回状态码
来源：http://ezh.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://unc.jinqigufen.top

[R31] 局部变量
来源：http://wzb.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://fig.yanxiufei.cn

[R32] 参数个数校验
来源：http://jvm.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sem.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://nbq.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://afg.jlsjyb.cn

[R34] 退出时清理
来源：http://brc.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://xpm.hammf.cn

[R35] 后台执行并等待
来源：http://tcs.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ryj.zdbjq.cn

[R36] 并发执行多个任务
来源：http://vxu.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://guy.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://ttv.smart0.xyz

files=$(ls -1)
来源：http://ipf.yangfankeji.com

[R38] 管道串联
来源：http://qox.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://uqq.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://vtl.ivvv.top

cmd > out.log 2>&1
来源：http://snw.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://rkx.jqgufenzy.top

echo "log" >> out.log
来源：http://tal.bbcook.cn

[R41] 丢弃输出
来源：http://agr.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://btj.aizwys.cn

[R42] 输入重定向
来源：http://avl.quarkkingdee.top

wc -l < a.txt
来源：http://vsc.uphjek.com

[R43] 按名字查找文件
来源：http://oxa.xuanzx.com

find . -name "*.log" -type f
来源：http://ffn.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://cjz.birdmap.top

find . -mtime -7 -type f
来源：http://ypx.yangfankeji.com

[R45] 批量删除
来源：http://hhx.9152youxi.cn


<!-- 参考信息 -->