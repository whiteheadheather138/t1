代发 wailian999

CREATE TABLE users (
来源：http://bzx.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://djt.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://mte.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://jbl.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xvj.hcnkem.com

);
来源：http://zmk.xylfe.cn

[Q02] 创建带外键的表
来源：http://fxk.zhixingplan.top

CREATE TABLE orders (
来源：http://evk.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://roq.jlsjyb.cn

user_id INT NOT NULL,
来源：http://chz.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://yec.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://weg.zhijiandao.cn

);
来源：http://nrs.aizwys.cn

[Q03] 增加列
来源：http://epq.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ipa.feifeiyinyue.top

[Q04] 修改列类型
来源：http://vnt.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwm.jianghu66.top

[Q05] 重命名列
来源：http://pqh.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://riv.sjlbkw.cn

[Q06] 删除列
来源：http://ydq.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ygg.xuanzx.com

[Q07] 删除表
来源：http://kbw.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://oud.zdqjudy.top

[Q08] 创建普通索引
来源：http://lgf.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bng.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://uri.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rez.guannengcc.top

[Q10] 插入单行
来源：http://cfr.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://doj.jqgufenzy.top

[Q11] 一次插入多行
来源：http://bgn.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lex.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://rzg.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://yay.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aum.vehdjk.com

[Q13] 忽略重复插入
来源：http://ilv.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://etk.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://tfn.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aum.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jqs.jqgufenzy.top

[Q15] 查询全部
来源：http://jir.yvedp.cn

SELECT * FROM users;
来源：http://qdl.sjlbkw.cn

[Q16] 查询指定列
来源：http://xti.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://rns.nanxuanxn.top

[Q17] 条件查询
来源：http://xtm.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://swk.hcnkem.com

[Q18] 模糊匹配
来源：http://zwr.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://whs.zycfv.cn

[Q19] 范围查询
来源：http://rau.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vym.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://yrz.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hck.sxryk.cn

[Q21] 空值判断
来源：http://oay.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://flx.tianlin.xyz

[Q22] 排序
来源：http://gwn.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://arq.shanyushiyangkeji.top

[Q23] 分页
来源：http://duf.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hxo.aizwys.cn

[Q24] 去重
来源：http://cul.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://bof.fehbvm.com

[Q25] 只取前 N 条
来源：http://snl.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cti.cheryme.top

[Q26] 计数
来源：http://llu.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://voo.hcnkem.com

[Q27] 条件计数
来源：http://wez.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://azb.316326.xyz

[Q28] 求和与平均
来源：http://ygz.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oux.cashguo.top

[Q29] 最大最小值
来源：http://dgx.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ita.fengsongda.top

[Q30] 分组统计
来源：http://bgp.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mkd.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://nym.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pjd.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://gsn.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cbp.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eiu.fanxiaobao.xyz

[Q33] 多列分组
来源：http://stp.316326.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vbk.gzhubu.top

[Q34] 每组取第一条
来源：http://xcp.yj202588.top

SELECT * FROM (
来源：http://stb.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ccs.jinqigufen.top

) t WHERE rn = 1;
来源：http://asn.9152youxi.cn

[Q35] 内连接
来源：http://jtr.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zsz.tarul.cn

[Q36] 左连接
来源：http://did.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ziy.52xcode.cn

[Q37] 右连接
来源：http://dvs.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ldj.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://qro.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fyn.hammf.cn

[Q39] 自连接（查上下级）
来源：http://gtr.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uts.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://owm.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qip.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lvi.gotoacloud.top

[Q41] 多表连接
来源：http://kqa.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tuw.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://hcc.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://suu.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://eqk.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://fhg.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tru.xinyue.icu

[Q43] 标量子查询
来源：http://kya.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mee.tarul.cn

[Q44] IN 子查询
来源：http://yil.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkp.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://kec.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfq.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cjw.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ebl.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://qzs.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cyh.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://cuw.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://siz.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://tlm.ppjwa.cn

[Q49] 更新单行
来源：http://fox.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wwf.ctjpmb.com

[Q50] 批量更新
来源：http://pty.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rgt.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://thc.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xvo.hnqzz.top

[Q52] 删除指定行
来源：http://urs.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://hry.zdbjq.cn

[Q53] 按条件删除
来源：http://szv.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vuc.jinyuanbaomall.cn

[Q54] 清空表
来源：http://kzi.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://txa.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://jxn.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vgq.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://knc.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hfe.yangfankeji.com

[Q57] 行号
来源：http://gmx.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xmc.quarkkingdee.top

[Q58] 累计求和
来源：http://jcm.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ipj.tianlin.xyz

[Q59] 分组内累计
来源：http://avj.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://boo.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://acf.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lfz.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gfy.ehwqpu.com

[Q61] 移动平均
来源：http://hui.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpz.ctjpmb.com

[Q62] 分组占比
来源：http://vuf.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yuw.jqgfzy.top

[Q63] 开启事务
来源：http://xxg.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nyz.snrcjt.cn

[Q64] 提交事务
来源：http://whd.ydjk.org.cn

COMMIT;
来源：http://izt.zdqjudy.top

[Q65] 回滚事务
来源：http://kph.shzxlz.cn

ROLLBACK;
来源：http://kfo.jianghu66.top

[Q66] 行锁查询
来源：http://ihb.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xqg.yvedp.cn

[Q67] 设置隔离级别
来源：http://ogc.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dnp.zhiwuduotai.top

[Q68] 保存点
来源：http://vyg.jiagoushi.top

SAVEPOINT sp1;
来源：http://bjm.meibo888.top

ROLLBACK TO sp1;
来源：http://pju.yueranfly.top

[Q69] 查看执行计划
来源：http://npx.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rav.sweek.top

[Q70] 更新统计信息
来源：http://gdg.52xcode.cn

ANALYZE TABLE users;
来源：http://rxz.zhoulong.xyz

[Q71] 查看建表语句
来源：http://ffe.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jzw.guannengcc.top

[Q72] 查看索引
来源：http://ikj.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://bth.cqqwz.cn

[Q73] 查看表状态
来源：http://xlv.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ede.fktsv.cn

[Q74] 强制使用索引
来源：http://qwa.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://div.tanke756.top

[Q75] 日期格式化
来源：http://zjf.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iwp.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yeq.tarul.cn

[Q76] 按天统计
来源：http://cvb.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://stf.hywenlv.cn

[Q77] 时间加减
来源：http://buz.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vzt.hnqzz.top

[Q78] 当前时间
来源：http://don.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fed.daxiang520.top

[Q79] 字符串拼接
来源：http://bxo.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qia.jqgufenzy.top

[Q80] 字符串截取
来源：http://vgw.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://inj.cheryme.top

[Q81] 字符串替换
来源：http://udj.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rgh.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://nco.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xoo.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://wbj.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qcr.jiagoushi.top

[Q84] 去除首尾空格
来源：http://kbb.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://zyr.jiagoushi.top

[Q85] 数值取整
来源：http://opw.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cmq.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://wrx.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ing.yj20258.top

[Q87] JSON 字段做条件
来源：http://hzz.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rnn.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://tay.yonumen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oll.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qag.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://gev.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dln.zdqjudy.top

[Q90] 生成序号列
来源：http://afn.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xih.ybcxt.top

================================================================================
来源：http://mib.yj20258888.top

R. Bash 专题
来源：http://yhd.jlsjyb.cn

================================================================================
来源：http://ahp.c1oappe.top

[R01] shebang 与严格模式
来源：http://lgy.tarul.cn

#!/usr/bin/env bash
来源：http://cax.jinqigfzy.top

set -euo pipefail
来源：http://ftz.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://msj.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://xuh.redwolf501.top

[R03] 只读变量
来源：http://tqh.uphjek.com

readonly PI=3.14
来源：http://cjn.daxiang520.top

[R04] 位置参数
来源：http://gqn.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://osi.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://iis.jlsjyb.cn

name="${1:-default}"
来源：http://jrn.hnqzz.top

[R06] 判断命令是否存在
来源：http://bjp.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbm.bjfxy.top

[R07] if 判断文件
来源：http://jds.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yme.0kj1m.cn

[R08] 数值比较
来源：http://qes.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fcv.daxiang520.top

[R09] 字符串比较
来源：http://mcb.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aim.fzhhl.top

[R10] 正则匹配
来源：http://lth.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bkt.chenlongwang.top

[R11] case 多分支
来源：http://tbu.bjfxy.top

case "$1" in
来源：http://foy.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://wcj.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://jqh.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://rbv.bbcook.cn

esac
来源：http://cry.yonumen.top

[R12] for 遍历文件
来源：http://oue.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://yfl.nanxinkj.top

[R13] for 计数循环
来源：http://mvg.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://fql.pycfn.com

[R14] C 风格 for
来源：http://jgx.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fin.fengsongda.top

[R15] while 逐行读文件
来源：http://zhx.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://snt.sweek.top

[R16] until 等待条件
来源：http://hfo.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://equ.zdbjq.cn

[R17] 数组定义与取值
来源：http://mpr.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://lwf.xinyue.icu

[R18] 遍历数组
来源：http://yze.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vaq.yangfankeji.com

[R19] 数组长度
来源：http://vtn.zhengqikj.top

echo "${#arr[@]}"
来源：http://ksl.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://iqd.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zqj.zhengqikj.top

[R21] 字符串长度
来源：http://ucl.redwolf501.top

echo "${#s}"
来源：http://xry.daxiang520.top

[R22] 截取子串
来源：http://gar.gaohongyu789.top

echo "${s:0:5}"
来源：http://bmr.wangshuangyany.cn

[R23] 字符串替换
来源：http://vwi.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kcl.nanxuanxn.top

[R24] 大小写转换
来源：http://ypc.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://lhm.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://nja.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rlp.guannengcc.top

[R26] 命令替换
来源：http://mho.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://nlg.wangshuangyany.cn

[R27] 算术展开
来源：http://fqe.sweek.top

echo $((1 + 2 * 3))
来源：http://iyv.feifeiyinyue.top

[R28] 浮点运算
来源：http://qrh.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://rih.cdnleiting.top

[R29] 定义函数
来源：http://fxp.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fuo.uphjek.com

[R30] 函数返回状态码
来源：http://ned.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://dgf.haohaochexian.top

[R31] 局部变量
来源：http://jnf.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://pgp.snrcjt.cn

[R32] 参数个数校验
来源：http://pmg.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qka.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://zsx.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://onp.shzxlz.cn

[R34] 退出时清理
来源：http://ajn.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://htu.tarul.cn

[R35] 后台执行并等待
来源：http://jzh.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ppi.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://emn.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bnr.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://jqz.jinyuanbaomall.cn

files=$(ls -1)
来源：http://cbb.jinghuilouyu.cn

[R38] 管道串联
来源：http://hwh.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://unj.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://jte.zhoulong.xyz

cmd > out.log 2>&1
来源：http://tnu.dianchejie.cn

[R40] 追加写日志
来源：http://twu.quarkkingdee.top

echo "log" >> out.log
来源：http://ndq.hammf.cn

[R41] 丢弃输出
来源：http://eyk.mhx1999.top

cmd >/dev/null 2>&1
来源：http://prx.pengpengdd.cyou

[R42] 输入重定向
来源：http://den.gaohongyu789.top

wc -l < a.txt
来源：http://jbj.zhengqikj.top

[R43] 按名字查找文件
来源：http://yra.tanke756.top

find . -name "*.log" -type f
来源：http://len.0kj1m.cn

[R44] 按修改时间查找
来源：http://sen.zhijiandao.cn

find . -mtime -7 -type f
来源：http://zxk.hnxiangtu.top

[R45] 批量删除
来源：http://ksj.fengsongda.top


<!-- 参考信息 -->