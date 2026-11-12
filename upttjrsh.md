代发 wailian999

CREATE TABLE users (
来源：http://gzg.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ehl.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://pzb.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://icd.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://maj.chenjidiqi.icu

);
来源：http://uld.jianghu66.top

[Q02] 创建带外键的表
来源：http://ofu.bbcook.cn

CREATE TABLE orders (
来源：http://sos.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pjj.zdbjq.cn

user_id INT NOT NULL,
来源：http://kna.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://kyh.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fvp.yanxiufei.cn

);
来源：http://lzh.iojbl.cn

[Q03] 增加列
来源：http://chp.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xnc.bjfxy.top

[Q04] 修改列类型
来源：http://jmg.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ghy.fengsongda.top

[Q05] 重命名列
来源：http://moc.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oug.feifeiyinyue.top

[Q06] 删除列
来源：http://hnu.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://xsm.52xcode.cn

[Q07] 删除表
来源：http://upi.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://tje.aizwys.cn

[Q08] 创建普通索引
来源：http://hip.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cvr.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://zud.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hlz.wangdashe.top

[Q10] 插入单行
来源：http://xxq.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ywi.ctjpmb.com

[Q11] 一次插入多行
来源：http://rgo.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pty.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://yuo.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cuw.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eht.yvedp.cn

[Q13] 忽略重复插入
来源：http://fed.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://slb.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://oai.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xqc.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vcr.fanxiaobao.xyz

[Q15] 查询全部
来源：http://yfy.tian-w.cn

SELECT * FROM users;
来源：http://aqs.shzxlz.cn

[Q16] 查询指定列
来源：http://fzg.redwolf501.top

SELECT id, name FROM users;
来源：http://bub.yonumen.top

[Q17] 条件查询
来源：http://rma.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://apf.hnqzz.top

[Q18] 模糊匹配
来源：http://ymd.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ycr.tianlin.xyz

[Q19] 范围查询
来源：http://bes.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hne.ydjk.org.cn

[Q20] IN 列表
来源：http://mpp.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zhm.chenzaomai.com

[Q21] 空值判断
来源：http://nvd.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hrc.zycfv.cn

[Q22] 排序
来源：http://vqv.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wia.cqqwz.cn

[Q23] 分页
来源：http://wlh.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzn.yangfankeji.com

[Q24] 去重
来源：http://hli.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://tdy.snrcjt.cn

[Q25] 只取前 N 条
来源：http://som.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gyl.tian-w.cn

[Q26] 计数
来源：http://vmo.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://vyg.smart0.xyz

[Q27] 条件计数
来源：http://bzm.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dbg.guowangkeji.top

[Q28] 求和与平均
来源：http://rmn.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wlp.birdmap.top

[Q29] 最大最小值
来源：http://atu.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gij.9152youxi.cn

[Q30] 分组统计
来源：http://hvc.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://swm.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://uya.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uun.tian-w.cn

[Q32] 分组拼接字符串
来源：http://mny.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qzs.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wwe.shanyushiyangtech.top

[Q33] 多列分组
来源：http://cjf.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kjp.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://yqs.sjlbkw.cn

SELECT * FROM (
来源：http://dkf.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jvv.jyoumei.cn

) t WHERE rn = 1;
来源：http://ady.jinyuanbaomall.cn

[Q35] 内连接
来源：http://tkg.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zle.chenzaomai.com

[Q36] 左连接
来源：http://vty.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nzk.tianlin.xyz

[Q37] 右连接
来源：http://kgw.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://scz.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://snt.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mle.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://iuk.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wfs.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kjv.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iey.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rxt.zycfv.cn

[Q41] 多表连接
来源：http://oaj.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zqm.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://vwy.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://ded.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://yqw.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://jxq.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yef.yuanzhike.top

[Q43] 标量子查询
来源：http://zba.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kce.daxiang520.top

[Q44] IN 子查询
来源：http://ejn.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yoj.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://kzk.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhf.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ika.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xep.jqgufenzy.top

[Q47] 与平均值比较
来源：http://nay.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ojp.pycfn.com

[Q48] CTE 公用表表达式
来源：http://ebg.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iyh.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://inp.iojbl.cn

[Q49] 更新单行
来源：http://eqn.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hdx.smart0.xyz

[Q50] 批量更新
来源：http://uqc.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xxx.zdqjudy.top

[Q51] 用子查询更新
来源：http://wlc.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nlz.ivvv.top

[Q52] 删除指定行
来源：http://bnz.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://wmp.gzhubu.top

[Q53] 按条件删除
来源：http://ees.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://efz.vehdjk.com

[Q54] 清空表
来源：http://ptq.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://eix.hammf.cn

[Q55] 排名（并列占位）
来源：http://wov.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ocj.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://frx.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rvw.hysaishi.cn

[Q57] 行号
来源：http://jhm.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swl.shanyushiyangtech.top

[Q58] 累计求和
来源：http://jcj.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xhl.jlsjyb.cn

[Q59] 分组内累计
来源：http://lui.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kzo.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://cml.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://srk.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qij.shanyushiyangtech.top

[Q61] 移动平均
来源：http://pbe.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gfm.shangyingyoupin.top

[Q62] 分组占比
来源：http://agj.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://piq.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://utl.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ixj.shzxlz.cn

[Q64] 提交事务
来源：http://gls.chenlongwang.top

COMMIT;
来源：http://jsp.cheryme.top

[Q65] 回滚事务
来源：http://zyp.zhijiandao.cn

ROLLBACK;
来源：http://dez.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://pin.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ndr.fktsv.cn

[Q67] 设置隔离级别
来源：http://whe.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nos.bjfxy.top

[Q68] 保存点
来源：http://ghi.svipenyu.cn

SAVEPOINT sp1;
来源：http://jxm.jqgfzy.top

ROLLBACK TO sp1;
来源：http://dcy.316326.xyz

[Q69] 查看执行计划
来源：http://xeb.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://poj.vehdjk.com

[Q70] 更新统计信息
来源：http://ijt.chenzaomai.com

ANALYZE TABLE users;
来源：http://fga.dianchejie.cn

[Q71] 查看建表语句
来源：http://qbd.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rus.daria6918.cn

[Q72] 查看索引
来源：http://ktf.aizwys.cn

SHOW INDEX FROM users;
来源：http://wmv.fengsongda.top

[Q73] 查看表状态
来源：http://rfn.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jnm.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://pze.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iqm.birdmap.top

[Q75] 日期格式化
来源：http://ivm.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uci.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hgi.ydjk.org.cn

[Q76] 按天统计
来源：http://nno.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ugr.jqgfzy.top

[Q77] 时间加减
来源：http://xfc.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vsc.nanxuanxn.top

[Q78] 当前时间
来源：http://lvf.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rad.tianlin.xyz

[Q79] 字符串拼接
来源：http://jjw.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqf.zhongyouzk.top

[Q80] 字符串截取
来源：http://uku.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lhw.cheryme.top

[Q81] 字符串替换
来源：http://bfl.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://smj.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://myy.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mdv.ctjpmb.com

[Q83] 大小写转换
来源：http://zql.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://taz.gzhubu.top

[Q84] 去除首尾空格
来源：http://orb.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://qkk.zhengqikj.top

[Q85] 数值取整
来源：http://xhv.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wsq.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://pdv.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://elc.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://daj.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nst.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://ggw.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oyv.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mav.nanxinkj.top

[Q89] 判断表是否存在
来源：http://ahx.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dbr.iojbl.cn

[Q90] 生成序号列
来源：http://lun.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://try.yueranfly.top

================================================================================
来源：http://wqp.zdqjudy.top

R. Bash 专题
来源：http://ggd.sufxvd.cn

================================================================================
来源：http://uow.yonumen.top

[R01] shebang 与严格模式
来源：http://vef.bjfxy.top

#!/usr/bin/env bash
来源：http://fqa.gaohongyu789.top

set -euo pipefail
来源：http://zfj.meibo888.top

[R02] 变量赋值与使用
来源：http://jzx.zdqjudy.top

name="Tom"; echo "$name"
来源：http://gtx.gaohongyu789.top

[R03] 只读变量
来源：http://mfs.hesvh.cn

readonly PI=3.14
来源：http://ltw.ppjwa.cn

[R04] 位置参数
来源：http://fel.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mdl.fengsongda.top

[R05] 参数默认值
来源：http://zsj.hywenlv.cn

name="${1:-default}"
来源：http://eed.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://wry.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://akm.yj20258888.top

[R07] if 判断文件
来源：http://pxi.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lpc.xinyue.icu

[R08] 数值比较
来源：http://wfh.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ojs.daxiang520.top

[R09] 字符串比较
来源：http://gjj.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gvp.kuanghao11.cn

[R10] 正则匹配
来源：http://mwu.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ags.gotoacloud.top

[R11] case 多分支
来源：http://vfy.52xcode.cn

case "$1" in
来源：http://xev.aibaodan.cn

start) echo "启动" ;;
来源：http://ugv.haohaochexian.top

stop)  echo "停止" ;;
来源：http://wja.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://udd.gogol.net.cn

esac
来源：http://vai.shangyingyoupin.top

[R12] for 遍历文件
来源：http://ztr.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://vmm.gaohongyu789.top

[R13] for 计数循环
来源：http://vjd.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://hjt.zycfv.cn

[R14] C 风格 for
来源：http://gsc.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vof.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://noo.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tii.svipenyu.cn

[R16] until 等待条件
来源：http://dpi.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kdy.jiagoushi.top

[R17] 数组定义与取值
来源：http://uve.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://zrx.sufxvd.cn

[R18] 遍历数组
来源：http://mhz.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gik.ppjwa.cn

[R19] 数组长度
来源：http://zlv.ivvv.top

echo "${#arr[@]}"
来源：http://cye.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://szk.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mhu.hnqzz.top

[R21] 字符串长度
来源：http://stk.tanke756.top

echo "${#s}"
来源：http://yvi.hnxiangtu.top

[R22] 截取子串
来源：http://are.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://nrx.hysaishi.cn

[R23] 字符串替换
来源：http://xek.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gmm.iojbl.cn

[R24] 大小写转换
来源：http://odj.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://yyv.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://teb.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kyv.wangshuangyany.cn

[R26] 命令替换
来源：http://iby.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://cjn.zycfv.cn

[R27] 算术展开
来源：http://bbr.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://auf.yongpay.top

[R28] 浮点运算
来源：http://xmp.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://fzy.hywenlv.cn

[R29] 定义函数
来源：http://jkf.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://elz.cucudq.cn

[R30] 函数返回状态码
来源：http://zky.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://ouo.ybcxt.top

[R31] 局部变量
来源：http://kzc.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://abb.yuxming.cn

[R32] 参数个数校验
来源：http://lgl.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xcj.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://dzf.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jax.xinyue.icu

[R34] 退出时清理
来源：http://tcm.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://tqt.aizwys.cn

[R35] 后台执行并等待
来源：http://igm.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cza.yfazqb.com

[R36] 并发执行多个任务
来源：http://gzj.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zsz.gogol.net.cn

[R37] 把输出赋给变量
来源：http://ujq.tanke756.top

files=$(ls -1)
来源：http://bie.ywan-chungtsiang.top

[R38] 管道串联
来源：http://nbc.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://xgi.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://hww.yvedp.cn

cmd > out.log 2>&1
来源：http://hwi.shanyushiyangtech.top

[R40] 追加写日志
来源：http://wwe.zhengqikj.top

echo "log" >> out.log
来源：http://eoi.pengpengdd.cyou

[R41] 丢弃输出
来源：http://jed.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://mgm.ybcxt.top

[R42] 输入重定向
来源：http://ywo.jianghu66.top

wc -l < a.txt
来源：http://bxj.xinyue.icu

[R43] 按名字查找文件
来源：http://ctc.pycfn.com

find . -name "*.log" -type f
来源：http://odq.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://vdt.sweek.top

find . -mtime -7 -type f
来源：http://lae.cdnleiting.top

[R45] 批量删除
来源：http://bjf.jinqigfzy.top


<!-- 参考信息 -->