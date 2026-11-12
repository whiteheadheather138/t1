代发 wailian999

================================================================================
来源：http://oer.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qha.hywenlv.cn

================================================================================
来源：http://njg.havefunace.top

[Q01] 创建表
来源：http://fwx.epnwcf.com

CREATE TABLE users (
来源：http://gpz.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uvw.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://xnc.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://pst.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kdi.gogol.net.cn

);
来源：http://lup.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://ino.cucudq.cn

CREATE TABLE orders (
来源：http://lvf.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://afk.tarul.cn

user_id INT NOT NULL,
来源：http://kgo.pycfn.com

amount DECIMAL(10, 2),
来源：http://gxw.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vlb.jiagoushi.top

);
来源：http://lxj.tian-w.cn

[Q03] 增加列
来源：http://uws.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ols.bbcook.cn

[Q04] 修改列类型
来源：http://jbd.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lgi.zhijiandao.cn

[Q05] 重命名列
来源：http://phl.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://itt.hammf.cn

[Q06] 删除列
来源：http://rol.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kdz.hfpthk.cn

[Q07] 删除表
来源：http://zrk.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://roh.sysykeji.top

[Q08] 创建普通索引
来源：http://xqo.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gjv.sxryk.cn

[Q09] 创建唯一索引
来源：http://ivw.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yxt.shzxlz.cn

[Q10] 插入单行
来源：http://zdc.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wcz.guowangkeji.top

[Q11] 一次插入多行
来源：http://jjo.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dbb.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://qkp.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pqr.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ioo.jiagoushi.top

[Q13] 忽略重复插入
来源：http://auo.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://afy.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://azq.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nil.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://idz.shangyingyoupin.top

[Q15] 查询全部
来源：http://bkm.zhixingplan.top

SELECT * FROM users;
来源：http://trx.fehbvm.com

[Q16] 查询指定列
来源：http://xuk.jqgufenzy.top

SELECT id, name FROM users;
来源：http://ojv.xinyue.icu

[Q17] 条件查询
来源：http://vwc.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cch.chenlongwang.top

[Q18] 模糊匹配
来源：http://ljf.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jwb.zhongyouzk.top

[Q19] 范围查询
来源：http://lwr.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tdx.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://pha.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ldl.xinyue.icu

[Q21] 空值判断
来源：http://xan.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://clb.shuidangran.top

[Q22] 排序
来源：http://etm.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ejk.dashuyun.cn

[Q23] 分页
来源：http://ziq.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://abk.316326.xyz

[Q24] 去重
来源：http://zey.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://vmo.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://cts.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ngs.hywenlv.cn

[Q26] 计数
来源：http://dye.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://uvq.bbcook.cn

[Q27] 条件计数
来源：http://ths.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xaq.xinyue.icu

[Q28] 求和与平均
来源：http://gvw.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lot.mhx1999.top

[Q29] 最大最小值
来源：http://kyn.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xoh.jqgfzy.top

[Q30] 分组统计
来源：http://oai.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sfd.pycfn.com

[Q31] 分组后过滤
来源：http://ybj.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ogh.aizwys.cn

[Q32] 分组拼接字符串
来源：http://yeo.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ino.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hnm.yj20258.top

[Q33] 多列分组
来源：http://gyn.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lnl.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://mqj.shanyushiyangtech.top

SELECT * FROM (
来源：http://xac.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://onl.nanxinkj.top

) t WHERE rn = 1;
来源：http://fjh.hcnkem.com

[Q35] 内连接
来源：http://ytb.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lbp.sufxvd.cn

[Q36] 左连接
来源：http://fmc.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tfm.chenzaomai.com

[Q37] 右连接
来源：http://rdf.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wgm.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://wfg.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qch.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://hrh.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wkp.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bcb.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sbi.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ckz.cucudq.cn

[Q41] 多表连接
来源：http://ikr.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ydz.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://rvo.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://yyt.yonumen.top

[Q42] 连接条件附加过滤
来源：http://vbm.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://rzj.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zgm.daria6918.cn

[Q43] 标量子查询
来源：http://shf.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pcx.hnxiangtu.top

[Q44] IN 子查询
来源：http://ejm.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pxt.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://upi.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qat.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vys.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qhs.guannengcc.top

[Q47] 与平均值比较
来源：http://zmi.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uoz.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://cse.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dfv.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://ugk.gzhubu.top

[Q49] 更新单行
来源：http://izu.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cwj.xuetiantiany.cn

[Q50] 批量更新
来源：http://eam.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vxr.birdmap.top

[Q51] 用子查询更新
来源：http://wgi.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yji.tianlin.xyz

[Q52] 删除指定行
来源：http://hzh.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://ebe.daria6918.cn

[Q53] 按条件删除
来源：http://bmh.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wqs.svipenyu.cn

[Q54] 清空表
来源：http://nll.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://iqk.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://zei.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lzm.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://shd.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qgg.zhoulong.xyz

[Q57] 行号
来源：http://ayx.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://api.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://ujr.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xev.zhoulong.xyz

[Q59] 分组内累计
来源：http://xws.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pcd.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://tfc.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://szt.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://scx.redwolf501.top

[Q61] 移动平均
来源：http://tcw.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gqx.hnqzz.top

[Q62] 分组占比
来源：http://hok.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfy.fanxiaobao.xyz

[Q63] 开启事务
来源：http://zas.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tnp.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://jbc.svipenyu.cn

COMMIT;
来源：http://icn.yj20258.top

[Q65] 回滚事务
来源：http://tai.chenjidiqi.icu

ROLLBACK;
来源：http://vhx.sufxvd.cn

[Q66] 行锁查询
来源：http://yik.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwv.cashguo.top

[Q67] 设置隔离级别
来源：http://rrd.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ylr.zhiwuduotai.top

[Q68] 保存点
来源：http://bda.zhoulong.xyz

SAVEPOINT sp1;
来源：http://usz.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://aqv.jiagoushi.top

[Q69] 查看执行计划
来源：http://igk.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hbu.pycfn.com

[Q70] 更新统计信息
来源：http://bjs.smart0.xyz

ANALYZE TABLE users;
来源：http://iba.havefunace.top

[Q71] 查看建表语句
来源：http://kzt.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aow.jiagoushi.top

[Q72] 查看索引
来源：http://lca.hesvh.cn

SHOW INDEX FROM users;
来源：http://qtq.yj20258888.top

[Q73] 查看表状态
来源：http://ber.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nau.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://zab.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iok.jqgufenzy.top

[Q75] 日期格式化
来源：http://cua.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://anu.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kwj.yongpay.top

[Q76] 按天统计
来源：http://szk.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qpn.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://uly.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rnj.shanyushiyangtech.top

[Q78] 当前时间
来源：http://idi.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vzq.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://afy.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bxw.yongpay.top

[Q80] 字符串截取
来源：http://que.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vvo.dashuyun.cn

[Q81] 字符串替换
来源：http://qbg.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dpq.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://ste.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fjg.zdqjudy.top

[Q83] 大小写转换
来源：http://ejc.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nkr.hysaishi.cn

[Q84] 去除首尾空格
来源：http://aky.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://tvi.hongshengwenyu.top

[Q85] 数值取整
来源：http://tfx.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hka.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://hbs.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wpo.ivvv.top

[Q87] JSON 字段做条件
来源：http://baa.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pkk.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://kop.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ndz.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://euf.xuanzx.com

[Q89] 判断表是否存在
来源：http://ite.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rhu.shuidangran.top

[Q90] 生成序号列
来源：http://uek.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vpj.yongpay.top

================================================================================
来源：http://vbe.fehbvm.com

R. Bash 专题
来源：http://cpl.fzhhl.top

================================================================================
来源：http://ldh.fktsv.cn

[R01] shebang 与严格模式
来源：http://vgj.andypj.xyz

#!/usr/bin/env bash
来源：http://yqp.chenzaomai.com

set -euo pipefail
来源：http://xzy.snrcjt.cn

[R02] 变量赋值与使用
来源：http://leq.chenzaomai.com

name="Tom"; echo "$name"
来源：http://eey.fengsongda.top

[R03] 只读变量
来源：http://nit.birdmap.top

readonly PI=3.14
来源：http://lhs.snrcjt.cn

[R04] 位置参数
来源：http://ijr.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aex.zycfv.cn

[R05] 参数默认值
来源：http://svn.andypj.xyz

name="${1:-default}"
来源：http://zby.jiagoushi.top

[R06] 判断命令是否存在
来源：http://lqg.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bnt.hongshengwenyu.top

[R07] if 判断文件
来源：http://dwh.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://voc.yanxiufei.cn

[R08] 数值比较
来源：http://fwe.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://pjr.dianchejie.cn

[R09] 字符串比较
来源：http://nzs.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://myp.jqgfzy.top

[R10] 正则匹配
来源：http://mkm.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uon.daria6918.cn

[R11] case 多分支
来源：http://mgl.ydjk.org.cn

case "$1" in
来源：http://ssz.hammf.cn

start) echo "启动" ;;
来源：http://jsd.ydzc1.top

stop)  echo "停止" ;;
来源：http://wis.mhx1999.top

*)     echo "未知命令" ;;
来源：http://doy.xziqi.cn

esac
来源：http://omn.jqgfzy.top

[R12] for 遍历文件
来源：http://yud.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://ktm.9152youxi.cn

[R13] for 计数循环
来源：http://vlq.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://nrp.yonumen.top

[R14] C 风格 for
来源：http://lmc.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://clo.redwolf501.top

[R15] while 逐行读文件
来源：http://urs.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xfl.guannengcc.top

[R16] until 等待条件
来源：http://nmy.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dhn.cucudq.cn

[R17] 数组定义与取值
来源：http://onr.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://afb.ybcxt.top

[R18] 遍历数组
来源：http://ndr.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kjw.jqgufenzy.top

[R19] 数组长度
来源：http://hcz.vqdsnc.cn

echo "${#arr[@]}"
来源：http://azi.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://lno.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://whn.zhiwuduotai.top

[R21] 字符串长度
来源：http://nku.jianghu66.top

echo "${#s}"
来源：http://qmf.zdqjudy.top

[R22] 截取子串
来源：http://qtw.jyoumei.cn

echo "${s:0:5}"
来源：http://xnm.yuxming.cn

[R23] 字符串替换
来源：http://mcj.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nkf.jlsjyb.cn

[R24] 大小写转换
来源：http://nqg.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://qmj.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://xry.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://pcg.aibaodan.cn

[R26] 命令替换
来源：http://ntl.316326.xyz

now=$(date +%F); echo "$now"
来源：http://ugb.zhoulong.xyz

[R27] 算术展开
来源：http://pnf.xylfe.cn

echo $((1 + 2 * 3))
来源：http://kai.guowangkeji.top

[R28] 浮点运算
来源：http://nop.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://nzz.hysaishi.cn

[R29] 定义函数
来源：http://yyd.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sku.tanke756.top

[R30] 函数返回状态码
来源：http://amr.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://rfp.jinqigfzy.top

[R31] 局部变量
来源：http://spm.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://wwa.hongshengwenyu.top

[R32] 参数个数校验
来源：http://svx.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xga.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://ysu.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sbh.xuetiantiany.cn

[R34] 退出时清理
来源：http://wyc.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://hjl.zycfv.cn

[R35] 后台执行并等待
来源：http://mqc.daxiang520.top

sleep 5 & pid=$!; wait "$pid"
来源：http://obt.hesvh.cn

[R36] 并发执行多个任务
来源：http://qpg.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jsp.andypj.xyz

[R37] 把输出赋给变量
来源：http://ukk.xylfe.cn

files=$(ls -1)
来源：http://iub.yuxming.cn

[R38] 管道串联
来源：http://iqu.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://adb.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://iqj.chenlongwang.top

cmd > out.log 2>&1
来源：http://qzx.c1oappe.top

[R40] 追加写日志
来源：http://xmw.xuanzx.com

echo "log" >> out.log
来源：http://tjr.hcnkem.com

[R41] 丢弃输出
来源：http://kpg.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://uor.zhoulong.xyz

[R42] 输入重定向
来源：http://tlx.zdqjudy.top

wc -l < a.txt
来源：http://bos.yj202588.top

[R43] 按名字查找文件
来源：http://hbs.yvedp.cn


<!-- 参考信息 -->