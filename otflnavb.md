代发 wailian999

================================================================================
来源：http://erx.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ehd.hnxiangtu.top

================================================================================
来源：http://ibg.jiagoushi.top

[Q01] 创建表
来源：http://zyg.tanke756.top

CREATE TABLE users (
来源：http://yel.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tlt.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://jll.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://tii.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bwa.sysykeji.top

);
来源：http://zzm.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://pul.cdnleiting.top

CREATE TABLE orders (
来源：http://mix.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyx.hysaishi.cn

user_id INT NOT NULL,
来源：http://zwq.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://xaw.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tnd.iojbl.cn

);
来源：http://gut.hongshengwenyu.top

[Q03] 增加列
来源：http://rji.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pfw.meibo888.top

[Q04] 修改列类型
来源：http://tji.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nae.fehbvm.com

[Q05] 重命名列
来源：http://kun.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cji.kuanghao11.cn

[Q06] 删除列
来源：http://qio.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://ynl.cucudq.cn

[Q07] 删除表
来源：http://euo.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://fun.meibo888.top

[Q08] 创建普通索引
来源：http://vcb.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://qwa.9152youxi.cn

[Q09] 创建唯一索引
来源：http://inq.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jri.cashguo.top

[Q10] 插入单行
来源：http://rwh.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zja.dashuyun.cn

[Q11] 一次插入多行
来源：http://psj.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ius.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://ktl.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fse.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mmk.tanke756.top

[Q13] 忽略重复插入
来源：http://hum.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mwz.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://byy.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aoj.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dux.gotoacloud.top

[Q15] 查询全部
来源：http://cll.cdnleiting.top

SELECT * FROM users;
来源：http://hrd.snrcjt.cn

[Q16] 查询指定列
来源：http://naj.jinqigfzy.top

SELECT id, name FROM users;
来源：http://ynj.hongshengwenyu.top

[Q17] 条件查询
来源：http://eto.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kzo.zhoulong.xyz

[Q18] 模糊匹配
来源：http://keg.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://unw.havefunace.top

[Q19] 范围查询
来源：http://rvy.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://guy.fktsv.cn

[Q20] IN 列表
来源：http://rpz.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vsu.xuanzx.com

[Q21] 空值判断
来源：http://btn.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://utf.jiagoushi.top

[Q22] 排序
来源：http://adr.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sis.vehdjk.com

[Q23] 分页
来源：http://kux.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhr.guannengcc.top

[Q24] 去重
来源：http://anj.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://wsl.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://ddi.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nna.sufxvd.cn

[Q26] 计数
来源：http://mlj.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://hgm.pengpengdd.cyou

[Q27] 条件计数
来源：http://mzm.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aib.chenlongwang.top

[Q28] 求和与平均
来源：http://rms.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yhm.gzhubu.top

[Q29] 最大最小值
来源：http://ell.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://suh.snrcjt.cn

[Q30] 分组统计
来源：http://qqq.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tcq.andypj.xyz

[Q31] 分组后过滤
来源：http://fku.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bhw.yonumen.top

[Q32] 分组拼接字符串
来源：http://ezr.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fmw.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tmx.ppjwa.cn

[Q33] 多列分组
来源：http://saw.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yua.fengsongda.top

[Q34] 每组取第一条
来源：http://krp.jiagoushi.top

SELECT * FROM (
来源：http://qij.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wmm.guowangkeji.top

) t WHERE rn = 1;
来源：http://dtr.iojbl.cn

[Q35] 内连接
来源：http://mci.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jyo.chenjidiqi.icu

[Q36] 左连接
来源：http://xqo.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yuf.cheryme.top

[Q37] 右连接
来源：http://yvm.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qtg.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ezh.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://svl.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://kfk.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hvp.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cyv.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zay.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ozc.0kj1m.cn

[Q41] 多表连接
来源：http://ivi.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lhq.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://nbx.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://eil.meibo888.top

[Q42] 连接条件附加过滤
来源：http://zux.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://bnu.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gyp.shangyingyoupin.top

[Q43] 标量子查询
来源：http://orl.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mcu.sweek.top

[Q44] IN 子查询
来源：http://uln.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gst.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://dfu.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ssm.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://xqi.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wdd.fzhhl.top

[Q47] 与平均值比较
来源：http://cyh.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sbl.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://nrl.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kov.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://iig.xylfe.cn

[Q49] 更新单行
来源：http://rrz.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uto.nanxinkj.top

[Q50] 批量更新
来源：http://hrm.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ckk.hywenlv.cn

[Q51] 用子查询更新
来源：http://yhl.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pjr.pycfn.com

[Q52] 删除指定行
来源：http://rmb.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://mrw.epnwcf.com

[Q53] 按条件删除
来源：http://cqi.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xby.bbcook.cn

[Q54] 清空表
来源：http://oxp.yonumen.top

TRUNCATE TABLE logs;
来源：http://muq.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://syv.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jlk.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://sdl.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvc.xylfe.cn

[Q57] 行号
来源：http://pab.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lpd.andypj.xyz

[Q58] 累计求和
来源：http://khf.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vjf.yuxming.cn

[Q59] 分组内累计
来源：http://eyo.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ktw.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://wdh.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ssp.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://old.daxiang520.top

[Q61] 移动平均
来源：http://pqi.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nos.sysykeji.top

[Q62] 分组占比
来源：http://nro.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nml.hesvh.cn

[Q63] 开启事务
来源：http://iwk.0kj1m.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iyo.9152youxi.cn

[Q64] 提交事务
来源：http://idj.birdmap.top

COMMIT;
来源：http://jog.nanxinkj.top

[Q65] 回滚事务
来源：http://csp.sxryk.cn

ROLLBACK;
来源：http://wfc.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://qfj.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uvu.yangfankeji.com

[Q67] 设置隔离级别
来源：http://hlq.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wvj.ydzc1.top

[Q68] 保存点
来源：http://gzo.hysaishi.cn

SAVEPOINT sp1;
来源：http://irm.uphjek.com

ROLLBACK TO sp1;
来源：http://eba.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://zig.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cha.jqgufenzy.top

[Q70] 更新统计信息
来源：http://tkk.fktsv.cn

ANALYZE TABLE users;
来源：http://kzu.yonumen.top

[Q71] 查看建表语句
来源：http://dho.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tru.yfazqb.com

[Q72] 查看索引
来源：http://vin.316326.xyz

SHOW INDEX FROM users;
来源：http://ije.kuanghao11.cn

[Q73] 查看表状态
来源：http://uuu.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ojj.zhongyouzk.top

[Q74] 强制使用索引
来源：http://doo.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dyi.hammf.cn

[Q75] 日期格式化
来源：http://wss.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yme.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bqp.tianlin.xyz

[Q76] 按天统计
来源：http://uxz.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qnp.chenzaomai.com

[Q77] 时间加减
来源：http://gwe.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gho.zhiwuduotai.top

[Q78] 当前时间
来源：http://bjw.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qyy.meibo888.top

[Q79] 字符串拼接
来源：http://gtl.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://npl.ivvv.top

[Q80] 字符串截取
来源：http://kff.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qhn.cdnleiting.top

[Q81] 字符串替换
来源：http://fml.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sua.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://hyp.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xyy.jqgfzy.top

[Q83] 大小写转换
来源：http://aki.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://whp.fzhhl.top

[Q84] 去除首尾空格
来源：http://hao.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://gvi.ydzc1.top

[Q85] 数值取整
来源：http://wlz.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ysa.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://edb.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kax.yfazqb.com

[Q87] JSON 字段做条件
来源：http://jqq.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ylt.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://eez.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://myj.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ihj.jinqigufen.top

[Q89] 判断表是否存在
来源：http://uyl.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qvp.aizwys.cn

[Q90] 生成序号列
来源：http://xho.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ppt.yanxiufei.cn

================================================================================
来源：http://gks.yj202588.top

R. Bash 专题
来源：http://dno.guowangkeji.top

================================================================================
来源：http://nbj.gogol.net.cn

[R01] shebang 与严格模式
来源：http://xkd.hesvh.cn

#!/usr/bin/env bash
来源：http://fyg.pengpengdd.cyou

set -euo pipefail
来源：http://rwr.fengsongda.top

[R02] 变量赋值与使用
来源：http://ylh.xziqi.cn

name="Tom"; echo "$name"
来源：http://gxw.daria6918.cn

[R03] 只读变量
来源：http://fes.iojbl.cn

readonly PI=3.14
来源：http://wex.yfazqb.com

[R04] 位置参数
来源：http://shz.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mrf.hammf.cn

[R05] 参数默认值
来源：http://qvz.zhoulong.xyz

name="${1:-default}"
来源：http://yki.daxiang520.top

[R06] 判断命令是否存在
来源：http://yyz.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lyg.redwolf501.top

[R07] if 判断文件
来源：http://loo.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnh.sxryk.cn

[R08] 数值比较
来源：http://siv.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dvu.sxryk.cn

[R09] 字符串比较
来源：http://zjz.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dmx.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://hxn.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bxo.zhengqikj.top

[R11] case 多分支
来源：http://ech.cdnleiting.top

case "$1" in
来源：http://ayk.jlsjyb.cn

start) echo "启动" ;;
来源：http://tnv.cdnleiting.top

stop)  echo "停止" ;;
来源：http://qul.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://hyr.zhiwuduotai.top

esac
来源：http://nal.sjlbkw.cn

[R12] for 遍历文件
来源：http://uaa.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://fwj.hammf.cn

[R13] for 计数循环
来源：http://mrz.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://xgx.aizwys.cn

[R14] C 风格 for
来源：http://lpw.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nfj.guannengcc.top

[R15] while 逐行读文件
来源：http://lpj.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kwz.shuidangran.top

[R16] until 等待条件
来源：http://bgn.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwo.iojbl.cn

[R17] 数组定义与取值
来源：http://oxx.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://xyw.tarul.cn

[R18] 遍历数组
来源：http://xoq.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rfw.xuanzx.com

[R19] 数组长度
来源：http://hfg.hnqzz.top

echo "${#arr[@]}"
来源：http://yob.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://xxw.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ioh.dashuyun.cn

[R21] 字符串长度
来源：http://loo.pycfn.com

echo "${#s}"
来源：http://ied.9152youxi.cn

[R22] 截取子串
来源：http://hap.zhongyouzk.top

echo "${s:0:5}"
来源：http://lkl.nanxuanxn.top

[R23] 字符串替换
来源：http://ila.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fzs.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://mth.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://fzx.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://ktd.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lqm.cheryme.top

[R26] 命令替换
来源：http://vxj.tanke756.top

now=$(date +%F); echo "$now"
来源：http://nlo.wangshuangyany.cn

[R27] 算术展开
来源：http://vir.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://pcg.jlsjyb.cn

[R28] 浮点运算
来源：http://jal.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://jii.vqdsnc.cn

[R29] 定义函数
来源：http://fdk.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mvp.yuxming.cn

[R30] 函数返回状态码
来源：http://zok.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://dfv.redwolf501.top

[R31] 局部变量
来源：http://kfb.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://nnp.jqgfzy.top

[R32] 参数个数校验
来源：http://zcx.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uyt.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://dgn.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tms.cashguo.top

[R34] 退出时清理
来源：http://rcm.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://txn.hcnkem.com

[R35] 后台执行并等待
来源：http://wqg.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eqh.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://thh.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fwi.zdqjudy.top

[R37] 把输出赋给变量
来源：http://nqm.fzhhl.top

files=$(ls -1)
来源：http://mmt.wangshuangyany.cn

[R38] 管道串联
来源：http://uwy.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://yhk.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://gav.cheryme.top

cmd > out.log 2>&1
来源：http://ldh.daxiang520.top

[R40] 追加写日志
来源：http://kuq.jinghuilouyu.cn

echo "log" >> out.log
来源：http://cqk.tanke756.top

[R41] 丢弃输出
来源：http://lgf.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://fpk.havefunace.top

[R42] 输入重定向
来源：http://rir.sxryk.cn

wc -l < a.txt
来源：http://mvv.svipenyu.cn

[R43] 按名字查找文件
来源：http://azq.uphjek.com


<!-- 参考信息 -->